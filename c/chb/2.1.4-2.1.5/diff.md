# Comparing `tmp/chb-2.1.4.tar.gz` & `tmp/chb-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chb-2.1.4.tar", last modified: Fri Apr  7 06:50:08 2023, max compression
+gzip compressed data, was "chb-2.1.5.tar", last modified: Thu Apr 20 15:10:23 2023, max compression
```

## Comparing `chb-2.1.4.tar` & `chb-2.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 06:50:08.266107 chb-2.1.4/
--rw-rw-rw-   0        0        0     1091 2023-04-07 05:55:28.000000 chb-2.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      637 2023-04-07 06:50:08.266107 chb-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-07 05:55:28.000000 chb-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 06:50:08.261121 chb-2.1.4/chb/
--rw-rw-rw-   0        0        0     5471 2023-04-07 05:55:28.000000 chb-2.1.4/chb/__init__.py
--rw-rw-rw-   0        0        0     8353 2023-04-07 06:49:37.000000 chb-2.1.4/chb/_dao.py
--rw-rw-rw-   0        0        0     3424 2023-04-07 05:55:28.000000 chb-2.1.4/chb/_importable.py
--rw-rw-rw-   0        0        0     3977 2023-04-07 05:55:28.000000 chb-2.1.4/chb/_imports.py
--rw-rw-rw-   0        0        0     4644 2023-04-07 05:55:28.000000 chb-2.1.4/chb/_log.py
--rw-rw-rw-   0        0        0    24576 2023-04-07 05:55:28.000000 chb-2.1.4/chb/_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 06:50:08.264113 chb-2.1.4/chb.egg-info/
--rw-rw-rw-   0        0        0      637 2023-04-07 06:50:08.000000 chb-2.1.4/chb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-07 06:50:08.000000 chb-2.1.4/chb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 06:50:08.000000 chb-2.1.4/chb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-07 06:50:08.000000 chb-2.1.4/chb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-07 06:50:08.266107 chb-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-04-07 06:50:00.000000 chb-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:10:23.952567 chb-2.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-07 05:55:28.000000 chb-2.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      637 2023-04-20 15:10:23.952567 chb-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-07 05:55:28.000000 chb-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 15:10:23.948342 chb-2.1.5/chb/
+-rw-rw-rw-   0        0        0     5471 2023-04-07 05:55:28.000000 chb-2.1.5/chb/__init__.py
+-rw-rw-rw-   0        0        0     8851 2023-04-20 15:09:42.000000 chb-2.1.5/chb/_dao.py
+-rw-rw-rw-   0        0        0     3424 2023-04-07 05:55:28.000000 chb-2.1.5/chb/_importable.py
+-rw-rw-rw-   0        0        0     3977 2023-04-07 05:55:28.000000 chb-2.1.5/chb/_imports.py
+-rw-rw-rw-   0        0        0     4644 2023-04-07 05:55:28.000000 chb-2.1.5/chb/_log.py
+-rw-rw-rw-   0        0        0    25832 2023-04-20 15:04:31.000000 chb-2.1.5/chb/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:10:23.951569 chb-2.1.5/chb.egg-info/
+-rw-rw-rw-   0        0        0      637 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 15:10:23.953564 chb-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-04-20 15:04:31.000000 chb-2.1.5/setup.py
```

### Comparing `chb-2.1.4/LICENSE.txt` & `chb-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chb-2.1.4/PKG-INFO` & `chb-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chb
-Version: 2.1.4
+Version: 2.1.5
 Summary: chb常用代码库
 Home-page: https://github.com/ChenHuabin321/pypi
 Author: chenhuabin
 Author-email: chenhuabin321@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chb-2.1.4/chb/__init__.py` & `chb-2.1.5/chb/__init__.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.4/chb/_dao.py` & `chb-2.1.5/chb/_dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,7 +241,25 @@
         self.db.hset(set_name, key, value)
 
     def hget(self, set_name, key):
         """
         从名为set_name的hash队列中获取一个键值对
         """
         return self.db.hget(set_name, key)
+
+    def sadd(self, set_name, value):
+        """
+        向名为set_name的set中添加一个元素value
+        """
+        self.db.sadd(set_name, value)
+
+    def srem(self, set_name, value):
+        """
+        向名为set_name的set中删除一个元素value
+        """
+        self.db.srem(set_name, value)
+
+    def inset(self, set_name, value):
+        """
+        判断元素value是否在名为set_name的set中
+        """
+        self.db.sismember(set_name, value)
```

### Comparing `chb-2.1.4/chb/_importable.py` & `chb-2.1.5/chb/_importable.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.4/chb/_imports.py` & `chb-2.1.5/chb/_imports.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.4/chb/_log.py` & `chb-2.1.5/chb/_log.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.4/chb/_utils.py` & `chb-2.1.5/chb/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -583,42 +583,76 @@
             lst = list(s)
             charLst = []
             for l in lst:
                 charLst.append(self.single_get_first(l))
             s2_list.append(''.join(charLst))
         return '_'.join(s2_list)
 
+
 class Cpen:
     """
-    无论文件是否存在都写入文件，功能待完善
+    打开或创建一个文件，并根据指定的模式进行读写。
+    如果文件不存在且使用非覆盖性写入模式，将自动创建一个新文件。
+
+    参数:
+    path: 文件路径
+    mode: 打开文件的模式
+    encoding: 文件编码，默认为 'utf-8'（仅适用于文本模式）
     """
+
     def __init__(self, path, mode, encoding='utf-8'):
         self.path = path
         self.mode = mode
-        if not os.path.exists(path):
-            with open(file=path, mode='w', encoding=encoding):
-                pass
-            self.f = open(file=path, mode=mode, encoding=encoding)
+        self.encoding = encoding
+
+        # 当文件不存在且使用非覆盖性写入模式时创建新文件
+        if not os.path.exists(path) and mode not in ('w', 'wb', 'w+', 'wb+', 'w+b'):
+            open(file=path, mode='w', encoding=encoding).close()
+
+        # 根据模式和编码打开文件
+        if 'b' in mode:  # 以二进制方式打开时，不能有mode参数
+            self.f = open(file=path, mode=mode)
         else:
             self.f = open(file=path, mode=mode, encoding=encoding)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.f.close()
 
+    def writeline(self, line):
+        """
+        在字符串末尾添加 \n 然后写入，如果是字节，则直接写入
+        :param line: 需要写入的字符串
+        """
+        if 'b' not in self.mode and isinstance(line, str):
+            self.f.write(line + '\n')
+        elif 'b' in self.mode and isinstance(line, bytes):
+            self.f.write(line)
+        else:
+            raise ValueError('输入内容类型与模式不匹配')
+
     def readline(self):
+        """
+        逐行读取文件内容，返回一个生成器。
+        """
         while True:
             line = self.f.readline()
             if not line:
                 break
             yield line
 
     def readlines(self, num_lines=100000):
+        """
+        按指定数量的行数读取文件内容，返回一个生成器。
+
+        参数:
+        num_lines: 每次读取的行数，默认为100000行
+        """
         while True:
             lines = self.f.readlines(num_lines)
             if not lines:
                 break
             yield lines
```

### Comparing `chb-2.1.4/chb.egg-info/PKG-INFO` & `chb-2.1.5/chb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chb
-Version: 2.1.4
+Version: 2.1.5
 Summary: chb常用代码库
 Home-page: https://github.com/ChenHuabin321/pypi
 Author: chenhuabin
 Author-email: chenhuabin321@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chb-2.1.4/setup.py` & `chb-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chb",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="2.1.4",  # 包版本号，便于维护版本
+    version="2.1.5",  # 包版本号，便于维护版本
     author="chenhuabin",  # 作者，可以写自己的姓名
     author_email="chenhuabin321@163.com",  # 作者联系方式，可写自己的邮箱地址
     description="chb常用代码库",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/ChenHuabin321/pypi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

