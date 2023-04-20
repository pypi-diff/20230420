# Comparing `tmp/win-basic-tools-0.3.3.tar.gz` & `tmp/win-basic-tools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win-basic-tools-0.3.3.tar", last modified: Fri Feb 24 00:10:18 2023, max compression
+gzip compressed data, was "win-basic-tools-0.3.4.tar", last modified: Thu Apr 20 12:10:31 2023, max compression
```

## Comparing `win-basic-tools-0.3.3.tar` & `win-basic-tools-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 00:10:18.680063 win-basic-tools-0.3.3/
--rw-rw-rw-   0        0        0     1093 2023-02-21 08:29:35.000000 win-basic-tools-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     1265 2023-02-24 00:10:18.680063 win-basic-tools-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      932 2023-02-04 05:43:45.000000 win-basic-tools-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-02-24 00:10:18.680063 win-basic-tools-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-02-23 23:59:20.000000 win-basic-tools-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 00:10:18.664434 win-basic-tools-0.3.3/win_basic_tools/
--rw-rw-rw-   0        0        0     8283 2023-02-22 04:12:55.000000 win-basic-tools-0.3.3/win_basic_tools/__init__.py
--rw-rw-rw-   0        0        0      304 2023-02-22 04:20:54.000000 win-basic-tools-0.3.3/win_basic_tools/__main__.py
--rw-rw-rw-   0        0        0     2132 2023-02-17 06:01:06.000000 win-basic-tools-0.3.3/win_basic_tools/setup_cmd.py
-drwxrwxrwx   0        0        0        0 2023-02-24 00:10:18.680063 win-basic-tools-0.3.3/win_basic_tools.egg-info/
--rw-rw-rw-   0        0        0     1265 2023-02-24 00:10:18.000000 win-basic-tools-0.3.3/win_basic_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-02-24 00:10:18.000000 win-basic-tools-0.3.3/win_basic_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 00:10:18.000000 win-basic-tools-0.3.3/win_basic_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-02-24 00:10:18.000000 win-basic-tools-0.3.3/win_basic_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-02-24 00:10:18.000000 win-basic-tools-0.3.3/win_basic_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-24 00:10:18.000000 win-basic-tools-0.3.3/win_basic_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/
+-rw-rw-rw-   0        0        0     1093 2023-02-21 08:29:35.000000 win-basic-tools-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     1265 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-02-04 05:43:45.000000 win-basic-tools-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-04-20 12:08:57.000000 win-basic-tools-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:10:31.649725 win-basic-tools-0.3.4/win_basic_tools/
+-rw-rw-rw-   0        0        0     8159 2023-04-20 12:05:40.000000 win-basic-tools-0.3.4/win_basic_tools/__init__.py
+-rw-rw-rw-   0        0        0      304 2023-02-22 04:20:54.000000 win-basic-tools-0.3.4/win_basic_tools/__main__.py
+-rw-rw-rw-   0        0        0     2132 2023-02-17 06:01:06.000000 win-basic-tools-0.3.4/win_basic_tools/setup_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/win_basic_tools.egg-info/
+-rw-rw-rw-   0        0        0     1265 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/top_level.txt
```

### Comparing `win-basic-tools-0.3.3/LICENSE` & `win-basic-tools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.3.3/PKG-INFO` & `win-basic-tools-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-basic-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Gives some small tools for shells on Windows
 Home-page: https://github.com/HenriquedoVal/win-basic-tools
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `win-basic-tools-0.3.3/README.md` & `win-basic-tools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.3.3/setup.py` & `win-basic-tools-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     page_description = f.read()
 
 with open('C:\\Users\\henri\\github\\win-basic-tools\\requirements.txt') as f:
     requirements = f.read()
 
 setup(
     name='win-basic-tools',
-    version='0.3.3',
+    version='0.3.4',
     author='Henrique do Val',
     author_email='henrique.val@hotmail.com',
     description='Gives some small tools for shells on Windows',
     long_description=page_description,
     long_description_content_type='text/markdown',
     url='https://github.com/HenriquedoVal/win-basic-tools',
     packages=find_packages(),
```

### Comparing `win-basic-tools-0.3.3/win_basic_tools/__init__.py` & `win-basic-tools-0.3.4/win_basic_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from io import StringIO
 import os
 import stat
 import sys
 import time
 
 from colorama import Fore, Style, deinit, init
 
@@ -53,24 +54,14 @@
         except PermissionError:
             return self.entry.is_dir(follow_symlinks=False)
 
     def is_symlink(self):
         return self.entry.is_symlink()
 
 
-class Cache:
-    __slots__ = 'data'
-
-    def __init__(self):
-        self.data = ''
-
-    def write(self, value):
-        self.data += value
-
-
 class Ls:
     '''
     Lists the content of a directory.
     '''
 
     __slots__ = 'opt', 'path', 'out', 'files', 'dirs', 'size'
 
@@ -79,15 +70,15 @@
         init()
 
         if not opt or opt.startswith('-'):
             self.opt, self.path = opt, path
         else:
             self.opt, self.path = '', opt
 
-        self.out = Cache() if to_cache else sys.stdout
+        self.out = StringIO() if to_cache else sys.stdout
         self.files = 0
         self.dirs = 0
         self.size = 0
 
     def __del__(self):
         deinit()
```

### Comparing `win-basic-tools-0.3.3/win_basic_tools/setup_cmd.py` & `win-basic-tools-0.3.4/win_basic_tools/setup_cmd.py`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.3.3/win_basic_tools.egg-info/PKG-INFO` & `win-basic-tools-0.3.4/win_basic_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-basic-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Gives some small tools for shells on Windows
 Home-page: https://github.com/HenriquedoVal/win-basic-tools
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

