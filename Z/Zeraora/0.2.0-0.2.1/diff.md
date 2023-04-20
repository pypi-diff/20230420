# Comparing `tmp/Zeraora-0.2.0.tar.gz` & `tmp/Zeraora-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.0.tar", last modified: Wed Apr 12 10:18:06 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.1.tar", last modified: Thu Apr 20 09:01:04 2023, max compression
```

## Comparing `Zeraora-0.2.0.tar` & `Zeraora-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:06.000000 Zeraora-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-12 10:18:06.000000 Zeraora-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-12 10:17:55.000000 Zeraora-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:18:06.000000 Zeraora-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-12 10:17:55.000000 Zeraora-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:06.000000 Zeraora-0.2.0/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:01:04.000000 Zeraora-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-20 09:01:04.000000 Zeraora-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-20 09:00:44.000000 Zeraora-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:01:04.000000 Zeraora-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-20 09:00:44.000000 Zeraora-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:01:04.000000 Zeraora-0.2.1/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/typing.py
```

### Comparing `Zeraora-0.2.0/PKG-INFO` & `Zeraora-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.0
+Version: 0.2.1
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
         
-        <div align="center"><i>长期维护的个人开源工具库<br>An utility Python package supports for my personal and company projects</i></div>
-        
-        [![Python](https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow)](https://docs.python.org/zh-cn/3/whatsnew/index.html) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://en.wikipedia.org/wiki/MIT_License) [![PyPI](https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI)](https://pypi.org/project/Zeraora/) ![conda](https://img.shields.io/conda/v/conda-forge/zeraora)
+        <div align="center">
+            <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow"></a>
+            <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
+            <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI"></a>
+            <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
+        </div>
+        <div align="center">
+            <i>长期维护的个人开源工具库</i>
+            <br>
+            <i>An utility Python package supports for my personal and company projects</i>
+        </div>
         
         ## Usage
         
         使用 pip 直接安装：
         
         ```shell
         pip install zeraora
@@ -42,15 +50,15 @@
         with BearTimer.BearTimer() as bear:
             summary = 0
             for i in range(1000000):
                 bear.step(f'loop to {i} now.')
                 summary += i
         ```
         
-        但对于 `charsets` 可以放心从子包导入：
+        但对于 `charsets` 和 `djangobase` 可以放心从子包导入：
         
         ```python
         from random import choices
         from zeraora.charsets import BASE64
         
         def make_pwd(length: int) -> str:
             return ''.join(choices(BASE64, k=length))
@@ -71,15 +79,15 @@
         
         ## Change
         
         > 仅列出不兼容旧版的修改，其余变动见git历史。
         
         ### 0.2.0（2023-4-12）
         
-        - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前面两个类。
+        - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Zeraora-0.2.0/README.md` & `Zeraora-0.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 <h1 align="center" style="padding-top: 32px">Zeraora</h1>
 
-<div align="center"><i>长期维护的个人开源工具库<br>An utility Python package supports for my personal and company projects</i></div>
-
-[![Python](https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow)](https://docs.python.org/zh-cn/3/whatsnew/index.html) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://en.wikipedia.org/wiki/MIT_License) [![PyPI](https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI)](https://pypi.org/project/Zeraora/) ![conda](https://img.shields.io/conda/v/conda-forge/zeraora)
+<div align="center">
+    <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow"></a>
+    <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
+    <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI"></a>
+    <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
+</div>
+<div align="center">
+    <i>长期维护的个人开源工具库</i>
+    <br>
+    <i>An utility Python package supports for my personal and company projects</i>
+</div>
 
 ## Usage
 
 使用 pip 直接安装：
 
 ```shell
 pip install zeraora
@@ -32,15 +40,15 @@
 with BearTimer.BearTimer() as bear:
     summary = 0
     for i in range(1000000):
         bear.step(f'loop to {i} now.')
         summary += i
 ```
 
-但对于 `charsets` 可以放心从子包导入：
+但对于 `charsets` 和 `djangobase` 可以放心从子包导入：
 
 ```python
 from random import choices
 from zeraora.charsets import BASE64
 
 def make_pwd(length: int) -> str:
     return ''.join(choices(BASE64, k=length))
@@ -61,8 +69,8 @@
 
 ## Change
 
 > 仅列出不兼容旧版的修改，其余变动见git历史。
 
 ### 0.2.0（2023-4-12）
 
-- 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前面两个类。
+- 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
```

### Comparing `Zeraora-0.2.0/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.1/Zeraora.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.0
+Version: 0.2.1
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
         
-        <div align="center"><i>长期维护的个人开源工具库<br>An utility Python package supports for my personal and company projects</i></div>
-        
-        [![Python](https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow)](https://docs.python.org/zh-cn/3/whatsnew/index.html) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://en.wikipedia.org/wiki/MIT_License) [![PyPI](https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI)](https://pypi.org/project/Zeraora/) ![conda](https://img.shields.io/conda/v/conda-forge/zeraora)
+        <div align="center">
+            <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow"></a>
+            <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
+            <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI"></a>
+            <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
+        </div>
+        <div align="center">
+            <i>长期维护的个人开源工具库</i>
+            <br>
+            <i>An utility Python package supports for my personal and company projects</i>
+        </div>
         
         ## Usage
         
         使用 pip 直接安装：
         
         ```shell
         pip install zeraora
@@ -42,15 +50,15 @@
         with BearTimer.BearTimer() as bear:
             summary = 0
             for i in range(1000000):
                 bear.step(f'loop to {i} now.')
                 summary += i
         ```
         
-        但对于 `charsets` 可以放心从子包导入：
+        但对于 `charsets` 和 `djangobase` 可以放心从子包导入：
         
         ```python
         from random import choices
         from zeraora.charsets import BASE64
         
         def make_pwd(length: int) -> str:
             return ''.join(choices(BASE64, k=length))
@@ -71,15 +79,15 @@
         
         ## Change
         
         > 仅列出不兼容旧版的修改，其余变动见git历史。
         
         ### 0.2.0（2023-4-12）
         
-        - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前面两个类。
+        - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Zeraora-0.2.0/setup.py` & `Zeraora-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.0/zeraora/charsets.py` & `Zeraora-0.2.1/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.0/zeraora/decorators.py` & `Zeraora-0.2.1/zeraora/decorators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.0/zeraora/generators.py` & `Zeraora-0.2.1/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.0/zeraora/time.py` & `Zeraora-0.2.1/zeraora/time.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.0/zeraora/typing.py` & `Zeraora-0.2.1/zeraora/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 mapper = annotations.get(attr, represent)
                 value = getattr(self, attr)
                 value = mapper(value) if callable(mapper) else value
                 yield f'{name}={value}'
 
         attributes = self.AttributeMeta.__dict__
         annotations = attributes.get('__annotations__', {})
-        return ' '.join(obtain())
+        return ' '.join(filter(None, obtain()))
 
     class TagMeta:
         """
         用于控制生成 representation 时需要带上哪些标签。
 
         注意：这个内部类不会被实例化！
 
@@ -243,15 +243,15 @@
                 elif isinstance(option, (list, dict)):
                     yield option[value]
                 else:
                     pass  # pragma: no cover
 
         attributes = self.TagMeta.__dict__
         annotations = attributes.get('__annotations__', {})
-        return ' '.join(obtain())
+        return ' '.join(filter(None, obtain()))
 
     def _obtain_pk(self) -> str:
         if hasattr(self, 'pk'):
             pk = self.pk
         elif hasattr(self, 'id'):
             pk = self.id
         else:
```

