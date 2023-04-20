# Comparing `tmp/isqopen-1.0.tar.gz` & `tmp/isqopen-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isqopen-1.0.tar", last modified: Mon Mar  6 03:39:49 2023, max compression
+gzip compressed data, was "isqopen-1.0.1.tar", last modified: Thu Apr 20 09:17:47 2023, max compression
```

## Comparing `isqopen-1.0.tar` & `isqopen-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,44 @@
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-03-06 03:39:49.000000 isqopen-1.0/
--rw-r--r--   0 huazhelou   (501) staff       (20)     1134 2023-03-06 03:39:49.000000 isqopen-1.0/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0/README.md
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-03-06 03:39:49.000000 isqopen-1.0/isq/
--rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2022-09-07 08:46:44.000000 isqopen-1.0/isq/QSyn.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    11379 2022-09-30 07:21:24.000000 isqopen-1.0/isq/Simplify.py
--rw-r--r--   0 huazhelou   (501) staff       (20)      215 2023-02-02 02:54:36.000000 isqopen-1.0/isq/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-02-02 02:22:27.000000 isqopen-1.0/isq/config.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5577 2023-03-06 03:23:39.000000 isqopen-1.0/isq/device.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2022-11-22 07:24:45.000000 isqopen-1.0/isq/errors.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     3846 2023-03-06 03:11:46.000000 isqopen-1.0/isq/globalVar.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1879 2022-12-02 03:43:49.000000 isqopen-1.0/isq/grad.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    10052 2022-11-17 10:23:55.000000 isqopen-1.0/isq/mapping.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2022-09-07 08:46:44.000000 isqopen-1.0/isq/matlab_gsvd.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     8644 2023-02-13 06:50:13.000000 isqopen-1.0/isq/operation.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    14833 2023-01-05 06:18:59.000000 isqopen-1.0/isq/parser.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    22701 2023-01-05 06:17:49.000000 isqopen-1.0/isq/parsetab.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    27546 2023-02-10 02:20:22.000000 isqopen-1.0/isq/passes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)      240 2022-11-14 09:19:11.000000 isqopen-1.0/isq/qpu.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5047 2022-09-07 08:46:44.000000 isqopen-1.0/isq/qtypes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6830 2023-02-21 08:20:11.000000 isqopen-1.0/isq/quantum.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     4622 2023-02-13 06:41:10.000000 isqopen-1.0/isq/simulator.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2679 2023-03-06 03:25:56.000000 isqopen-1.0/isq/task.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2180 2023-01-05 04:44:36.000000 isqopen-1.0/isq/tokrules.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2541 2022-09-30 07:24:21.000000 isqopen-1.0/isq/tools.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     3576 2023-03-06 03:19:48.000000 isqopen-1.0/isq/translate.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-03-06 03:39:49.000000 isqopen-1.0/isqopen.egg-info/
--rw-r--r--   0 huazhelou   (501) staff       (20)     1134 2023-03-06 03:39:49.000000 isqopen-1.0/isqopen.egg-info/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      550 2023-03-06 03:39:49.000000 isqopen-1.0/isqopen.egg-info/SOURCES.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-03-06 03:39:49.000000 isqopen-1.0/isqopen.egg-info/dependency_links.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-03-06 03:39:49.000000 isqopen-1.0/isqopen.egg-info/not-zip-safe
--rw-r--r--   0 huazhelou   (501) staff       (20)       70 2023-03-06 03:39:49.000000 isqopen-1.0/isqopen.egg-info/requires.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-03-06 03:39:49.000000 isqopen-1.0/isqopen.egg-info/top_level.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-03-06 03:39:49.000000 isqopen-1.0/setup.cfg
--rw-r--r--   0 huazhelou   (501) staff       (20)      803 2023-03-06 03:20:00.000000 isqopen-1.0/setup.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-03-06 03:39:49.000000 isqopen-1.0/test/
--rw-r--r--   0 huazhelou   (501) staff       (20)      761 2022-09-30 07:18:57.000000 isqopen-1.0/test/test.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.595718 isqopen-1.0.1/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2022-09-07 10:16:53.000000 isqopen-1.0.1/LICENSE
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-04-20 09:17:47.595852 isqopen-1.0.1/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0.1/README.md
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.587623 isqopen-1.0.1/isq/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      247 2023-04-17 07:47:49.000000 isqopen-1.0.1/isq/__init__.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.590577 isqopen-1.0.1/isq/compile/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/QSyn.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    11380 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/Simplify.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-17 07:26:56.000000 isqopen-1.0.1/isq/compile/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/matlab_gsvd.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    14686 2023-04-17 07:39:03.000000 isqopen-1.0.1/isq/compile/parser.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    22701 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/parsetab.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    27549 2023-04-17 07:28:07.000000 isqopen-1.0.1/isq/compile/passes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5050 2023-04-17 07:27:41.000000 isqopen-1.0.1/isq/compile/qtypes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2183 2023-04-17 07:28:19.000000 isqopen-1.0.1/isq/compile/tokrules.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2539 2023-04-17 07:38:44.000000 isqopen-1.0.1/isq/compile/tools.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/config.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.592009 isqopen-1.0.1/isq/device/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      142 2023-04-17 07:47:47.000000 isqopen-1.0.1/isq/device/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6293 2023-04-20 08:59:29.000000 isqopen-1.0.1/isq/device/device.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1882 2023-04-17 07:43:57.000000 isqopen-1.0.1/isq/device/grad.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2907 2023-04-17 07:45:20.000000 isqopen-1.0.1/isq/device/task.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     3578 2023-04-17 07:45:26.000000 isqopen-1.0.1/isq/device/translate.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.592799 isqopen-1.0.1/isq/draw/
+-rw-r--r--   0 huazhelou   (501) staff       (20)       26 2023-04-17 07:47:34.000000 isqopen-1.0.1/isq/draw/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     7986 2023-04-17 07:42:07.000000 isqopen-1.0.1/isq/draw/drawer.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/errors.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1221 2023-04-17 07:31:53.000000 isqopen-1.0.1/isq/globalVar.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)      250 2023-04-17 07:48:53.000000 isqopen-1.0.1/isq/qpu.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6707 2023-04-20 08:59:15.000000 isqopen-1.0.1/isq/quantum.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.593737 isqopen-1.0.1/isq/simulate/
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-17 07:29:05.000000 isqopen-1.0.1/isq/simulate/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    12918 2023-04-17 07:29:15.000000 isqopen-1.0.1/isq/simulate/operation.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5256 2023-04-17 07:28:56.000000 isqopen-1.0.1/isq/simulate/simulator.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.595488 isqopen-1.0.1/isqopen.egg-info/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      760 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/SOURCES.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/dependency_links.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/not-zip-safe
+-rw-r--r--   0 huazhelou   (501) staff       (20)       46 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/requires.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/top_level.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-04-20 09:17:47.596386 isqopen-1.0.1/setup.cfg
+-rw-r--r--   0 huazhelou   (501) staff       (20)      700 2023-04-20 09:10:33.000000 isqopen-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `isqopen-1.0/README.md` & `isqopen-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `isqopen-1.0/isq/QSyn.py` & `isqopen-1.0.1/isq/compile/QSyn.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0/isq/Simplify.py` & `isqopen-1.0.1/isq/compile/Simplify.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 if labT[j] == 1:
                     gateType.append('RY {}'.format(target))
                 elif labT[j] == 2:
                     val1 = labU[0,0,j]
                     val2 = labU[1,1,j]
                     theta = polar(val2)[1] - polar(val1)[1]
                     if isinstance(theta, complex):
-                        print(theta)
+                        #print(theta)
                         theta = theta.real
                     gateType.append('RZ({}) {}'.format(theta, target))
                 else:
                     #print(C)
                     if very_close(labU[:,:,j], H):
                         gateType.append('H {}'.format(target))
                     else:
```

### Comparing `isqopen-1.0/isq/device.py` & `isqopen-1.0.1/isq/device/device.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 from abc import ABC, abstractmethod
-from .errors import *
-from .parser import IR, compile
-from .config import debug_mode
-from .simulator import simulate, getprobs
-from .mapping import *
-from ezQpy import *
+from isq.errors import *
+from isq.compile.parser import IR, compile
+from isq.config import debug_mode
+from isq.simulate.simulator import simulate, getprobs
 import random
-from .quantum import quantumCor
+from isq.quantum import quantumCor
 from .translate import translate_to_aws, translate_to_qcis
 from .task import *
 from .grad import optv
+from isq.draw.drawer import Drawer
+import logging
+from isq.globalVar import isq_env
+
+try:
+    from ezQpy import *
+    isq_env.set_env('qcis', True)
+except:
+    pass
 
-from .globalVar import get_aws_support
 try:
     from braket import aws
 except:
     pass
 
 
 def getRandom():
     s = ""
     for _ in range(10):
         s += chr(random.randint(97, 122))
     return s
 
 class Device(ABC):
 
-    def __init__(self, name, shots = 1000, max_wait_time = 600):
+    def __init__(self, name, shots = 1000, max_wait_time = 600, logger=logging.getLogger(__name__)):
         self._name = name
         self._shots = shots
         self._max_wait_time = max_wait_time
         self._ir = ''
+        self.logger = logger
         pass
 
     @abstractmethod
     def run(self, isq_str = '', file = None,  **kwargs):
         pass
 
     def get_ir(self):
@@ -75,28 +82,33 @@
         for k,v in kwargs.items():
             if isinstance(v, optv):
                 args[k] = v._value
                 v = v._value
             kw[k] = v
         return args, kw
     
+    def draw_circuit(self, showparam=False):
+        if self._ir:
+            dw = Drawer(showparam=showparam)
+            dw.plot(self._ir)
+
     @property
     def shots(self):
         return self._shots
     
     @property
     def max_wait_time(self):
         return self._max_wait_time
         
 
 class LocalDevice(Device):
 
-    def __init__(self, shots = 100, max_wait_time = 60, name = None, mode = 'fast'):
+    def __init__(self, shots = 100, max_wait_time = 60, name = None, mode = 'fast', logger=logging.getLogger(__name__)):
         if name == None: name = "local_device"
-        super().__init__(name, shots, max_wait_time)
+        super().__init__(name, shots, max_wait_time, logger)
         
         if mode not in ['normal', 'fast']:
             raise CoreError('"{}" simulate mode is not support, only ["fast", "normal"]'.format(mode))
         self._mode = mode
 
 
     def run(self, isq_str = '', file = None, **kwargs):
@@ -115,61 +127,67 @@
         return getprobs(self._ir, mod, **args)
 
         
 
 
 class QcisDevice(Device):
 
-    def __init__(self, user, passwd, shots = 1000, max_wait_time = 60, name = None):
+    def __init__(self, user, passwd, shots = 1000, max_wait_time = 60, name = None, logger=logging.getLogger(__name__)):
         if name == None: name = "qcis_device"
-        super().__init__(name, shots, max_wait_time)
+        
+        if not isq_env.get_env('qcis'):
+            raise Exception("ezQpy is not supported in this env, please install ezQpy first")
+
+        super().__init__(name, shots, max_wait_time, logger)
 
         username = user
         password = passwd
-
+        
         self._account = Account(username=username, password=password, full_expr_record=True)
         self._qid = 0
     
     def run(self, isq_str = '', file = None, automap = False, init_map = None, **kwargs):
 
         qcis = self.compile_to_ir(isq_str, file, "qcis", **kwargs)
-        circuit = quantumCor.getMapping(12, [[1, 2], [2, 3], [3, 4], [4, 5], [5, 6], [6, 7], [7, 8], [8, 9], [9, 10], [10, 11], [11, 12]], qcis)
-        self._ir = circuit
+        #circuit = quantumCor.getMapping(12, [[1, 2], [2, 3], [3, 4], [4, 5], [5, 6], [6, 7], [7, 8], [8, 9], [9, 10], [10, 11], [11, 12]], qcis)
+        self._ir = qcis
 
         exp_name = "{}_{}".format(self._name, getRandom())
-        query_id = self._account.submit_job(circuit=circuit, exp_name=exp_name, version="1.0", num_shots=self._shots)
+        query_id = self._account.submit_job(circuit=qcis, exp_name=exp_name, version="1.0", num_shots=self._shots)
         if query_id:
-            print('qcis提交任务成功')
+            self.logger.info('qcis提交任务成功')
             return ISQTask(query_id, TaskType.QCSI, TaskState.WAIT, self)
         else:
-            print('qcis提交失败, 请确认硬件是否正常，或稍后再试')
+            self.logger.error('qcis提交失败, 请确认硬件是否正常，或稍后再试')
             return ISQTask(0, TaskType.QCSI, TaskState.FAIL, self)
 
 
 class AwsDevice(Device):
 
-    def __init__(self, device_arn, s3, shots = 1000, max_wait_time = 60, name = None):
+    def __init__(self, device_arn, s3, shots = 1000, max_wait_time = 60, name = None, logger=logging.getLogger(__name__)):
+        
+        if not isq_env.get_env('aws'):
+            raise Exception("aws is not supported in this env, please `pip install amazon-braket-sdk`")
+        
         if name == None: name = "aws_device"
-        super().__init__(name, shots, max_wait_time)
+        super().__init__(name, shots, max_wait_time, logger)
 
-        if not get_aws_support():
-            raise "aws is not support in this env, please `pip install amazon-braket-sdk`"
         #self._device = LocalSimulator()
         self._device = aws.AwsDevice(device_arn)
         self._s3_folder = s3
 
     
     def run(self, isq_str = '', file = None, **kwargs):
 
         isq_ir = self.compile_to_ir(isq_str, file, "isq", **kwargs)
         circuit, q_measure = translate_to_aws(isq_ir)
         self._ir = circuit
         try:
             task = self._device.run(circuit, self._s3_folder, shots=self._shots)
             #task = self._device.run(circuit, shots=self._shots)
-            print('aws提交任务成功')
-            return ISQTask(task.id, TaskType.AWS, TaskState.WAIT, self, measure = q_measure)
+            self.logger.info('aws提交任务成功')
+            return ISQTask(task.id, TaskType.AWS, TaskState.WAIT, self, measure = q_measure, logger =self.logger)
             
         except Exception as e:
-            print(str(e))
-            print('aws提交失败, 请确认硬件是否正常，或稍后再试')
+            self.logger.error(str(e))
+            self.logger.error('aws提交失败, 请确认硬件是否正常，或稍后再试')
             return ISQTask(0, TaskType.AWS, TaskState.FAIL, self)
```

### Comparing `isqopen-1.0/isq/errors.py` & `isqopen-1.0.1/isq/errors.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0/isq/grad.py` & `isqopen-1.0.1/isq/device/grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from autograd import numpy as anp
 from autograd.core import make_vjp as _make_vjp
 from autograd.extend import vspace
 from autograd.wrap_util import unary_to_nary
-from .errors import CoreError
+from isq.errors import CoreError
 from collections import Iterable
 
 class optv:
     def __init__(self, value = None):
         self._value = value
 
 class optimizer:
```

### Comparing `isqopen-1.0/isq/matlab_gsvd.py` & `isqopen-1.0.1/isq/compile/matlab_gsvd.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0/isq/parser.py` & `isqopen-1.0.1/isq/compile/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ply import (
     lex,
     yacc
 )
 import typing as T
 from typing import (cast, List, Any)
 from .qtypes import *
-from isq import tokrules
+from . import tokrules
 from .tokrules import tokens
-from .globalVar import varDic, msgDic
+from isq.globalVar import msgDic
 import numpy as np
 import sys
 import logging
-from .config import debug_mode
-from .errors import *
+from isq.config import debug_mode
+from isq.errors import *
 from .passes import PartialEvaluation
 import time
 
 
 current_line = 0
 current_ID = ''
 
@@ -443,21 +443,14 @@
 
         #print("now starting parsing")
 
         s = T.cast(Node, parser.parse(data, tracking = True))
         pre_time = trace_time(pre_time, "yacc")
         # if debug_mode == True:
         # print(s.type)
-
-        # if debug_mode == True:
-        # print(globalVar.varDic)
-
-        
-        if debug_mode == True:
-            print("paras: ", varDic)
         
         #s = passes.flatten_qbitdef_list(s)
         #globalVar.trace_time("flatten")
         mypass = PartialEvaluation(gate, par, target, args)
         ir.out = mypass.visitProgram(s)
         pre_time = trace_time(pre_time, "partial evaluation")
         #return 0
```

### Comparing `isqopen-1.0/isq/parsetab.py` & `isqopen-1.0.1/isq/compile/parsetab.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0/isq/passes.py` & `isqopen-1.0.1/isq/compile/passes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .qtypes import *
 import typing as T
 import copy
-from .errors import *
+from isq.errors import *
 import numpy as np
 import time
 from .tools import decompose
 
 """
 Flatten defBlock into a list of definitions.
 This makes qbitDef children Tuple[var_array|var] -> List[var_array|var]
```

### Comparing `isqopen-1.0/isq/qtypes.py` & `isqopen-1.0.1/isq/compile/qtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import (Literal, Tuple, Union, Protocol, Generic, TypeVar)
 import typing as T
 import types
-from .errors import ICE
+from isq.errors import ICE
 import inspect
 import sys
 
 ProcedureKey = str
 GateKey = str
 VarKey = str
 QbitType = Literal["qbit"]
```

### Comparing `isqopen-1.0/isq/quantum.py` & `isqopen-1.0.1/isq/quantum.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import sys
 from unittest.mock import patch
 import numpy as np
 from .errors import *
 import inspect
-from .parser import IR, compile
 from .config import debug_mode
-from .tools import decompose
-from .simulator import simulate
-from collections import defaultdict
-from .mapping import *
-from ezQpy import *
+from .compile.tools import decompose
 import random
 
 def getRandom():
     s = ""
     for i in range(10):
         s += chr(random.randint(97, 122))
     return s     
@@ -77,20 +72,22 @@
     def getGate():
         return quantumCor.__gate
 
     @staticmethod
     def getIR():
         return quantumCor.__ir
     
+    '''
     @staticmethod
     def getMapping(qubit_num, topo, isq_ir):
         init_map = get_init_map_by_reverse(qubit_num, topo, isq_ir)
         mp = Map(qubit_num, topo, isq_ir, init_map)
         return mp.mapping()
-    
+    '''
+
     '''
     @staticmethod
     def compileFromStr(isq_str, target='qcis', **kwargs):
         ir = IR()
         res = compile(ir, isq_str, target, quantumCor.__gate, kwargs)
         if res == -1:
             raise CoreError(ir.error)
```

### Comparing `isqopen-1.0/isq/simulator.py` & `isqopen-1.0.1/isq/simulate/simulator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from autograd import numpy as anp
 import time
-from .errors import *
+from isq.errors import *
 from collections import defaultdict
 from .operation import *
-from .globalVar import get_jax_env
+from isq.globalVar import isq_env
 
 gate_list = ['H', 'X', 'Y', 'Z', 'S', 'T', 'RZ', 'RX', 'RY', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P', 'CZ', 'CY', 'CX', 'CNOT', 'M']
 
 def check(line_data):
     
     qdic = {}
     qnum = 0
@@ -49,17 +49,26 @@
     return qnum, qdic
 
 def getstate(line_data, qnum, qdic, mod, **kwargs):
 
     state = anp.zeros(pow(2, qnum), dtype = complex)
     state[0] = 1
     
-    if get_jax_env() and mod:
-        state = jnp.zeros(jnp.power(2, qnum), dtype = complex)
-        state = state.at[0].set(1)
+    if mod == 1:
+        if isq_env.get_env('jax'):
+            state = jnp.zeros(jnp.power(2, qnum), dtype = complex)
+            state = state.at[0].set(1)
+        else:
+            raise Exception('jax is not supported in this env, please install jax first!')
+    elif mod == 2:
+        if isq_env.get_env('torch'):
+            state = torch.zeros(torch.pow(torch.tensor(2), torch.tensor(qnum)), dtype = torch.cfloat)
+            state[0] = 1
+        else:
+            raise Exception('torch is not supported in this env, please install torch first!')
 
     mq = []
     for idx, line in enumerate(line_data):
         line = line.strip()
         if not line:
             continue
         strArr = line.split(' ')
@@ -106,20 +115,28 @@
     line_data = data.split('\n')
 
     qnum, qdic = check(line_data)
 
     state, mq = getstate(line_data, qnum, qdic, mod, **kwargs)
     state = shift(state, qnum, mq)
 
-    if get_jax_env() and mod:
+    if mod==1:
         state = state.conj() * state
         n = len(mq)
         state = jnp.reshape(state, [1 << n, 1 << (qnum - n)])
         
         return jnp.real(jnp.sum(state, axis = 1))
+
+    elif mod==2:
+        state = state.conj() * state
+        n = len(mq)
+        state = torch.reshape(state, [1 << n, 1 << (qnum - n)])
+        
+        return torch.real(torch.sum(state, axis = 1))
+
     else:
         state = anp.conj(state) * state
         n = len(mq)
         state = anp.reshape(state, [1 << n, 1 << (qnum - n)])
         
         return anp.real(anp.sum(state, axis = 1))
```

### Comparing `isqopen-1.0/isq/task.py` & `isqopen-1.0.1/isq/device/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 try:
-    from .globalVar import aws_support, get_aws_support
+    from isq.globalVar import isq_env
     from braket.aws.aws_quantum_task import AwsQuantumTask
-    aws_support()
+    isq_env.set_env('aws', True)
 except:
     pass
 from typing import Union
+from logging import getLogger
 class TaskType:
     QCSI = "QCIS"
     AWS = "AWS"
 
 class TaskState:
     WAIT = "WAITING"
     COMPLETE = "COMPLETED"
@@ -22,18 +23,22 @@
     def __init__(self, task_id: Union[int, str], task_type, state, device, **kwargs) -> None:
         
         self._id = task_id
         self._type = task_type
         self._state = state
         self._res = {}
         self._device = device
+        self.logger = getLogger(__name__)
+        if 'logger' in kwargs:
+            self.logger = kwargs['logger']
         if self._type == TaskType.AWS and self._state not in self.NO_RESULT_TERMINAL_STATES:
-            if not get_aws_support():
+            if not isq_env.get_env('aws'):
                 raise "aws is not support in this env, please `pip install amazon-braket-sdk`"
-            self._task = AwsQuantumTask(self._id, poll_timeout_seconds = self._device._max_wait_time)
+    
+            self._task = AwsQuantumTask(self._id, poll_timeout_seconds = self._device._max_wait_time, logger=self.logger)
             self._measure = kwargs['measure']
 
     @property
     def state(self):
         return self._state
     
     def result(self):
@@ -41,41 +46,41 @@
             return {}
 
         if self._state == TaskState.COMPLETE: return self._res
         
         if self._type == TaskType.QCSI:
             m_res = self._device._account.query_experiment(self._id, max_wait_time = self._device._max_wait_time)
             if m_res:
-                print("任务执行成功")
+                self.logger.info("任务执行成功")
                 self._state = TaskState.COMPLETE
                 self._res = m_res
             else:
-                print("任务执行中，请等待")
+                self.logger.info("任务执行中，请等待")
         
         if self._type == TaskType.AWS:
             state = self._task.state()
             if state in self.NO_RESULT_TERMINAL_STATES:
-                print("任务已失败或已取消")
+                self.logger.info("任务已失败或已取消")
                 self._state = state
                 return {}
 
             m_res = self._task.result()
             if m_res:
-                print("任务执行成功")
+                self.logger.info("任务执行成功")
                 mc = m_res.measurement_counts
                 ans = {}
                 # get measure qbit
                 for k in mc:
                     rk = ''.join([k[i] for i in self._measure])
                     if rk not in ans: ans[rk] = 0
                     ans[rk] += mc[k]
                 self._res = ans
                 self._state = TaskState.COMPLETE
             else:
-                print("任务执行中，请等待")
+                self.logger.info("任务执行中，请等待")
 
         return self._res
 
     def cancel(self):
 
         if self._state == TaskState.WAIT:
             if self._type == TaskType.AWS:
```

### Comparing `isqopen-1.0/isq/tokrules.py` & `isqopen-1.0.1/isq/compile/tokrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .errors import CompileError
+from isq.errors import CompileError
 
 t_EQ  = r'\=\='
 t_LE  = r'\<\='
 t_GE  = r'\>\='
 t_NE = r'\!\='
 t_KET_ZERO = r'\|0\>'
 t_ignore = ' \t\r'
```

### Comparing `isqopen-1.0/isq/tools.py` & `isqopen-1.0.1/isq/compile/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from isq import QSyn, Simplify
+from . import QSyn, Simplify
 import numpy as np
 
 def decompose(mat, rowS, current_ID, pos = None):
 
         # add position info
         posstr = ""
         if pos != None:
```

### Comparing `isqopen-1.0/isq/translate.py` & `isqopen-1.0.1/isq/device/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numpy import pi
-from .globalVar import aws_support, get_aws_support
+from isq.globalVar import isq_env
 try:
     from braket.circuits import Circuit
-    aws_support()
+    isq_env.set_env('aws', True)
 except:
     pass
 
 QCIS_TO_AWS = {
     'H': 'h',
     'X': 'x',
     'Y': 'y',
@@ -43,15 +43,15 @@
                 res.append(f'CZ {qcis_tmp[1]} {qcis_tmp[2]}')
             else:
                 res.append(qcis)
     return "\n".join(res)
 
 def translate_to_aws(isq_ir):
     
-    if not get_aws_support():
+    if not isq_env.get_env('aws'):
         raise "aws is not support in this env, please `pip install amazon-braket-sdk`"
 
     circuit = Circuit()
     q_cnt = 0
     q_map = {}
     q_measure = []
```

### Comparing `isqopen-1.0/isqopen.egg-info/SOURCES.txt` & `isqopen-1.0.1/isqopen.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
-isq/QSyn.py
-isq/Simplify.py
 isq/__init__.py
 isq/config.py
-isq/device.py
 isq/errors.py
 isq/globalVar.py
-isq/grad.py
-isq/mapping.py
-isq/matlab_gsvd.py
-isq/operation.py
-isq/parser.py
-isq/parsetab.py
-isq/passes.py
 isq/qpu.py
-isq/qtypes.py
 isq/quantum.py
-isq/simulator.py
-isq/task.py
-isq/tokrules.py
-isq/tools.py
-isq/translate.py
+isq/compile/QSyn.py
+isq/compile/Simplify.py
+isq/compile/__init__.py
+isq/compile/matlab_gsvd.py
+isq/compile/parser.py
+isq/compile/parsetab.py
+isq/compile/passes.py
+isq/compile/qtypes.py
+isq/compile/tokrules.py
+isq/compile/tools.py
+isq/device/__init__.py
+isq/device/device.py
+isq/device/grad.py
+isq/device/task.py
+isq/device/translate.py
+isq/draw/__init__.py
+isq/draw/drawer.py
+isq/simulate/__init__.py
+isq/simulate/operation.py
+isq/simulate/simulator.py
 isqopen.egg-info/PKG-INFO
 isqopen.egg-info/SOURCES.txt
 isqopen.egg-info/dependency_links.txt
 isqopen.egg-info/not-zip-safe
 isqopen.egg-info/requires.txt
-isqopen.egg-info/top_level.txt
-test/test.py
+isqopen.egg-info/top_level.txt
```

### Comparing `isqopen-1.0/setup.py` & `isqopen-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "isqopen",
-    version = "1.0",
+    version = "1.0.1",
     keyword = {"isq", "quantum", "cor"},
     description = "isq quantum kernel",
     platforms='python 3.8+',
     long_description=long_description,
 	long_description_content_type="text/markdown",
     author = "Lou Huazhe",
     author_email = "louhz@arclightquantum.com",
 
     package_data = {'':['*.txt']},
     install_requires = ['numpy>=1.21.3',
                         'ply>=3.11',
                         'scipy>=1.7.1',
-                        'networkx>=2.3',
-                        'bs4',
-                        'ezQpy',
                         'autograd'],
     packages = find_packages(),
     zip_safe=False
 )
```

